# geoskill-building-footprint-height

> Extract building footprints and estimate height, floor count proxy, and volume from DSM/DTM/LiDAR data. Produces 2.5D urban models for 3D city modeling, population downscaling, and risk exposure analysis.

See [SKILL.md](SKILL.md) for full usage, inputs and outputs.

## Quick start

```bash
# Synthetic demo mode (no input files needed)
python scripts/building_footprint_height.py --output-dir ./bfh-output

# With custom floor height assumption
python scripts/building_footprint_height.py --floor-height 3.6 --output-dir ./bfh-output

# With point cloud method
python scripts/building_footprint_height.py --height-method point_cloud_quantile --output-dir ./bfh-output

# With custom standards
python scripts/building_footprint_height.py --standard-config ./my-standards.json --output-dir ./bfh-output
```

## License

MIT
