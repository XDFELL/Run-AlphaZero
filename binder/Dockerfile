FROM julia:1.8

COPY Project.toml .
COPY Manifest.toml .

RUN julia --project=. -e "using Pkg; Pkg.instantiate()"

COPY . .

CMD ["julia", "-e", "using AlphaZero"]
