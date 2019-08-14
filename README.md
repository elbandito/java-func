# java-func
riff Java function

# To run 

## Create riff builder
`pack create-builder elbandito/builder -b builder.toml --no-pull`

## Create java function image
`pack build elbandito/func --builder elbandito/builder -p ~/path/to/java-func --env RIFF=true --no-pull`

## Run
`docker run -i -p 8080:8080 elbandito/func`

# toml
You can omit passing the `--env RIFF=true` by creating a top level
`riff.toml` file as specified in the `/toml` directory.