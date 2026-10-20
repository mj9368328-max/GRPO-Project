# Run instructions

1. Open Google Colab: https://colab.research.google.com/
2. Upload `Jahid_Task05_GRPO_Unsloth.ipynb`.
3. Select **Runtime → Change runtime type → T4 GPU**.
4. Run each cell in order. Package versions may change; if a GRPO API mismatch appears, check the current Unsloth/TRL documentation and adapt the configuration.
5. Wait for training to finish. The notebook uses a compact 0.5B model, 4-bit loading, LoRA, 120 training examples, and 30 steps as a small demonstration.
6. Save the `reward_progression.png` plot and copy the generated sample output into the report.
7. Download the saved LoRA adapter folder if required.

## Notes
- A free Colab GPU can be unavailable or disconnect due to usage limits.
- Reward curves may fluctuate; they are not guaranteed to rise monotonically.
- The notebook's `AFTER TRAINING` output is genuine only after the training cell completes.
- For a real before/after comparison, generate a base-model answer before training (or load a fresh base model in a separate runtime) and compare on the same prompts.
