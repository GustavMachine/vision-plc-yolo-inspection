# Computer Vision Inspection System with YOLO + PLC

Sistema de visión por computadora para inspección automática de piezas,
integrado con PLC Beckhoff mediante ADS.

## Technologies
- Python
- OpenCV
- YOLO (Ultralytics)
- TensorFlow / PyTorch
- pyads (Beckhoff ADS)
- PLC Beckhoff (TwinCAT)

## Description
The system captures images from an IP camera,
runs YOLO-based classification,
and sends the result to a Beckhoff PLC using ADS communication.

A temporal voting mechanism over multiple frames is used
to improve robustness against noise and false positives.

## Workflow
PLC Trigger → Frame Capture → YOLO Inference → Temporal Voting → PLC Output

## Author
Gustavo Diego Espinoza Herrera
