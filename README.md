# 11ty
Step by step guide Create 11ty basic project


### install step by step
```
npm init -y
npm i --save-dev @11ty/eleventy
echo '# 11ty, Hello World!' > README.md
echo index.html
```

add this code to index.html
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>11ty</title>
    <style>
      body {
        font-family: BenchNine, system-ui, -apple-system, sans-serif;
        font-size: 3em;
        margin: 0 0 0.5em;
      }

      /*
      credit github user:
link: https://github.com/philipwalton/solved-by-flexbox/blob/master/demos/vertical-centering.md
      */
      .Aligner {
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .Aligner-item {
        flex: 1;
      }

      .Aligner-item--top {
        align-self: flex-start;
      }

      .Aligner-item--bottom {
        align-self: flex-end;
      }

      .Aligner-item--fixed {
        flex: none;
        text-align: center;
        margin-top: 10%;
      }
    </style>
  </head>
  <body>
    <div class="Aligner">
      <div class="Aligner-item Aligner-item--fixed">
        <h1>11ty, Hello World!</h1>
      </div>
    </div>
  </body>
</html>
```

Run

```
npx @11ty/eleventy --serve
```

##### [http://localhost:8080](http://localhost:8080/)

##### [http://localhost:8080/README/](http://localhost:8080/README/)
