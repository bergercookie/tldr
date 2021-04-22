# React

> Frontend shit

- Empty function in react component:

```typescriptreact
<CardActions className={classes.center}>
  <Button size="large" color="primary" onClick={() => void 0}>
      Download sample dataset
  </Button>
</CardActions>
```

- Instruct browser to download file on click

```typescriptreact
<CardActions className={classes.center}>
  <Button size="large" color="primary" onClick={() => window.location.assign("link to fetch it from") }>
    Download sample euroc dataset
  </Button>
</CardActions>
```
