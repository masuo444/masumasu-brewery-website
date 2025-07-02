# FOMUS Project - Masumasu Brewery

This directory contains a FOMUS music notation project for the Masumasu Brewery website.

## Files

- `example.fms` - Main FOMUS composition file with sample music
- `fomus.conf` - Configuration file for FOMUS settings
- `Makefile` - Build automation for generating different output formats
- `README.md` - This documentation file

## Requirements

- FOMUS music notation software must be installed
- Make utility (for using the Makefile)

## Usage

### Generate all formats:
```bash
make all
```

### Generate specific formats:
```bash
make xml    # Generate MusicXML
make lily   # Generate LilyPond
make midi   # Generate MIDI
```

### Clean generated files:
```bash
make clean
```

### Show help:
```bash
make help
```

## Output

Generated files will be placed in the `output/` directory:
- `masumasu-score.xml` - MusicXML format
- `masumasu-score.ly` - LilyPond format  
- `masumasu-score.mid` - MIDI format

## Customization

Edit `example.fms` to modify the musical composition. The current example includes:
- A simple melodic line inspired by traditional Japanese music
- Harmonic accompaniment
- Piano and strings instrumentation

Modify `fomus.conf` to change output settings, formatting, and other FOMUS parameters.