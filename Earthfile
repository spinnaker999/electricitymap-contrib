VERSION 0.6
FROM alpine:3.15
WORKDIR /contrib

dependencies:
  COPY pyproject.toml ./
  SAVE ARTIFACT .
  SAVE IMAGE contrib-dependencies:latest

config-files:
  COPY --dir config ./
  COPY --dir electricitymap/contrib/config ./electricitymap/contrib/config
  SAVE ARTIFACT .
  SAVE IMAGE contrib-config-files:latest

extras:
  COPY --dir electricitymap ./
  COPY --dir parsers ./
  COPY --dir validators ./
  SAVE ARTIFACT .
  SAVE IMAGE contrib-extras:latest
