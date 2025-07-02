# Makefile for FOMUS project - Masumasu Brewery

# Variables
FOMUS = fomus
CONFIG = fomus.conf
INPUT = example.fms
OUTPUT_DIR = output

# Default target
all: xml lily midi

# Create output directory
$(OUTPUT_DIR):
	mkdir -p $(OUTPUT_DIR)

# Generate MusicXML
xml: $(OUTPUT_DIR)
	$(FOMUS) -c $(CONFIG) -o $(OUTPUT_DIR)/masumasu-score.xml $(INPUT)

# Generate LilyPond
lily: $(OUTPUT_DIR)
	$(FOMUS) -c $(CONFIG) -o $(OUTPUT_DIR)/masumasu-score.ly $(INPUT)

# Generate MIDI
midi: $(OUTPUT_DIR)
	$(FOMUS) -c $(CONFIG) -o $(OUTPUT_DIR)/masumasu-score.mid $(INPUT)

# Clean generated files
clean:
	rm -rf $(OUTPUT_DIR)

# Show help
help:
	@echo "Available targets:"
	@echo "  all   - Generate all output formats (XML, LilyPond, MIDI)"
	@echo "  xml   - Generate MusicXML output"
	@echo "  lily  - Generate LilyPond output"
	@echo "  midi  - Generate MIDI output"
	@echo "  clean - Remove generated files"
	@echo "  help  - Show this help message"

.PHONY: all xml lily midi clean help