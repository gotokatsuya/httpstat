# httpstat

```sh
go get github.com/gotokatsuya/httpstat
```

```go
res, _ := httpstat.Request("GET", "{{ URL }}", nil, nil)
enc := json.NewEncoder(os.Stderr)
enc.SetIndent("", "  ")
enc.Encode(res.Stats())
```

This is 1.7 wrapper of github.com/apex/httpstat.
