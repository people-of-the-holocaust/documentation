
TARGET_PATH = main
PDF_NAME = document
ARTIFACT_DIR = .build_artifacts
OUTPUT_DIR = output
BUILD_FLAGS = -interaction=batchmode -output-directory=$(ARTIFACT_DIR) -jobname=$(PDF_NAME) $(TARGET_PATH)

build:
	mkdir -p $(ARTIFACT_DIR)
	mkdir -p $(OUTPUT_DIR)
	pdflatex $(BUILD_FLAGS) > /dev/null
	pdflatex $(BUILD_FLAGS) > /dev/null
	mv $(ARTIFACT_DIR)/$(PDF_NAME).pdf $(OUTPUT_DIR)/$(PDF_NAME).pdf
	@echo
	@echo "Build Log:  ./$(ARTIFACT_DIR)/$(PDF_NAME).log"
	@echo "PDF Output: ./$(OUTPUT_DIR)/$(PDF_NAME).pdf"

clean:
	rm -rf $(ARTIFACT_DIR)
