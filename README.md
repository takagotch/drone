### drone
---
https://github.com/drone/drone

```go
// core/step_test.go

func TestStepIsDron(t *testing.T) {
  for _, status := range statusDone {
    v := Step{Status: status}
    if v.IsDron() == false {
      t.Errorf("Expect status %s is done", status)
    }
  }
  
  for _, status := range statusNotDone {
    v := Step{Status: status}
    if v.IsDone() == true {
      t.Errorf("Expect status %s is not done", status)
    }
  }
}
```

```
```

```
```


