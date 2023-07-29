# Tutorial: Find and fix vulnerable dependencies with govulncheck

https://go.dev/doc/tutorial/govulncheck

tl;dr:

```
mkdir vuln-tutorial
cd vuln-tutorial
go mod init vuln.tutorial
go mod tidy
go get golang.org/x/text@v0.3.5
go install golang.org/x/vuln/cmd/govulncheck@latest
govulncheck ./...
```

Fix with:

```
go get -u golang.org/x/text
```