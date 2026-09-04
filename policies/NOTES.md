# Policy log
- uv run scripts/export.py Mjlab-Velocity-Flat-MicroDuck --checkpoint-file <path> --onnx-file policies/walk_v2_flat_8192env_XXXXiter.onnx
- nano policies/NOTES.md        # add a line about it
- git add policies/
- git commit -m "Add walk_v2"
- git push


- walk_v1_flat_4096env_23750iter — stock Mjlab-Velocity-Flat task, 4096 envs, stopped at 23750 iters. Walks well.
- walk_v2_flat_8192env_20500iter - stock Mjlab-Velocity-Flat tack, 8192 envs, stopped at 20550 iters. Much better walking
