# Policy log
- uv run scripts/export.py Mjlab-Velocity-Flat-MicroDuck --checkpoint-file <path> --onnx-file policies/walk_v2_flat_8192env_XXXXiter.onnx
- nano policies/NOTES.md        # add a line about it
- git add policies/
- git commit -m "Add walk_v2"
- git push


- walk_v1_flat_4096env_23750iter — stock Mjlab-Velocity-Flat task, 4096 envs, stopped at 23750 iters. Walks well.
- walk_v2_flat_8192env_20500iter - stock Mjlab-Velocity-Flat tack, 8192 envs, stopped at 20550 iters. Much better walking

echo "- standup_v1_flat_4096env_14999iter - Mjlab-StandUp-Flat-MicroDuck, 4096 envs, finished 15000 iters. Gets up from face-down/face-up/sitting in sim." >> policies/NOTES.md
echo "- walk_v3_flat_8192env_26499iter - resumed from v2 (20500), +6000 iters, 8192 envs. Walks fine; not yet compared with v2." >> policies/NOTES.md
git add policies/
git commit -m "Add standup_v1 and walk_v3"
git push
