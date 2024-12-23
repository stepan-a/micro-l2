all: examen-2024-2025-a.pdf correction-2024-2025-a.pdf

%.pdf: %.tex
	rubber --pdf $^
	rubber --clean $^
	rm -rf auto

clean-all:
	rm -f examen-2024-2025-a.pdf correction-2024-2025-a.pdf
