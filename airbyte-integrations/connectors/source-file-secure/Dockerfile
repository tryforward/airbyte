FROM airbyte/source-file:0.3.7

WORKDIR /airbyte/integration_code
COPY source_file_secure ./source_file_secure
COPY main.py ./
COPY setup.py ./
RUN pip install .

ENV AIRBYTE_ENTRYPOINT "python /airbyte/integration_code/main.py"
ENTRYPOINT ["python", "/airbyte/integration_code/main.py"]

LABEL io.airbyte.version=0.3.7
LABEL io.airbyte.name=airbyte/source-file-secure
