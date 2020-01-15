# installing node 

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash
nvm install node
```

proxy.lua

init = function(args)
    target_url = args[1] -- proxy needs absolute URL
end

request = function()
    return wrk.format("GET", target_url)
end
