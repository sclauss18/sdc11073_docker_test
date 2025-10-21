# Basis-Image
FROM python:3.12-slim

# Verhindere interaktive Abfragen
ENV DEBIAN_FRONTEND=noninteractive

# Installiere Abhängigkeiten
RUN pip install --no-cache-dir sdc11073==2.3.0

# Kopiere nur notwendige Dateien
COPY provider.py provider.py
COPY mdib.xml mdib.xml

ENTRYPOINT ["python", "provider.py"]
