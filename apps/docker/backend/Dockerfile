# 3.10.6

FROM python:3.10.6-slim-buster

WORKDIR /apps/backend

COPY ./apps/backend .

RUN python -m venv /opt/venv && \
    /opt/venv/bin/pip install --upgrade pip && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x /apps/backend/entrypoint.sh

CMD ["/apps/backend/entrypoint.sh"]