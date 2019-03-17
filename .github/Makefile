MDs := CODE_OF_CONDUCT.md \
    CODE_OF_CONDUCT_cn.md

GO := go

all: misspell toc


misspell:
	$(GO) get github.com/client9/misspell/cmd/misspell
	misspell \
		-locale GB \
		-error \
		*.md
toc:
	# brew install nodejs
	# npm install -g doctoc
	doctoc --title '' --github $(MDs)
