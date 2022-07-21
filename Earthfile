VERSION 0.6
FROM alpine:3.15
WORKDIR /contrib

files:
  COPY pyproject.toml ./
  COPY --dir config ./
  COPY --dir electricitymap/contrib/config ./electricitymap/contrib/config
  SAVE ARTIFACT .
  SAVE IMAGE contrib-files:latest
