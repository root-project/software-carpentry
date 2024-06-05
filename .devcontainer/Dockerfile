FROM rootproject/root:latest

RUN apt-get update && apt-get install -y git python3 python3-venv

RUN mkdir -p /py-venv \
 && python3 -m venv /py-venv/codespace \
 && /py-venv/codespace/bin/pip install --no-cache-dir --upgrade pip jupyter metakernel dask distributed pyspark

ENV PATH="/py-venv/codespace/bin:$PATH"
