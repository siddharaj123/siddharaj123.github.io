
CC = xelatex
RESUME_DIR = resume
OUTPUT_DIR = output
OUTPUT_FILENAME = Resume
RESUME_SRCS = $(shell find $(RESUME_DIR) -name '*.tex')
CV_SRCS = $(shell find $(CV_DIR) -name '*.tex')

resume.pdf: $(RESUME_DIR)/resume.tex $(RESUME_SRCS)
	$(CC) --jobname=$(OUTPUT_FILENAME) -output-directory=$(OUTPUT_DIR) $<
	rm $(OUTPUT_DIR)/$(OUTPUT_FILENAME).aux
	rm $(OUTPUT_DIR)/$(OUTPUT_FILENAME).log
	rm $(OUTPUT_DIR)/$(OUTPUT_FILENAME).out

clean:
	rm -rf $(OUTPUT_DIR)/*.pdf
