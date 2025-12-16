# GTFOBins

[![CI status](https://github.com/GTFOBins/GTFOBins.github.io/actions/workflows/ci.yml/badge.svg)](https://github.com/GTFOBins/GTFOBins.github.io/actions?query=workflow:CI)

GTFOBins is a curated list of Unix binaries that can be used to bypass local security restrictions in misconfigured systems.

### Repository purpose
- Educational purpose

### Credit
Find the project at https://gtfobins.github.io


### Run locally on terminal
- Replace old Gemfile.lock with the latest version of Gemfile.lock

```
.PHONY: serve serve-public bundle lint

serve:
	bundle exec jekyll serve

serve-public:
	bundle exec jekyll serve --host 0.0.0.0

bundle:
	bundle install

lint:
	yamllint _gtfobins/*.md
	scripts/validate-schema.py
```

