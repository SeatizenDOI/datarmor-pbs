
# Drone segment
Use [**the-point-is-the-mask**](https://github.com/SeatizenDOI/the-point-is-the-mask) for training.

The training process is divided into **three steps**:

1. **Initial training** of the model.
2. **Inference with SAM Refiner** — note that this step **cannot be run on Datarmor**, as `fastgeodis` is not installed.
3. **Retraining** the model using the outputs from the inference step.