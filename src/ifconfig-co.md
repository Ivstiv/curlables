# > $ curl ifconfig.co

![Example](img/ifconfig-co-thumbnail.png =600x)

## Description
Pretty simple to use tool to obtain various information about your network as observed from an outside party. Go to their 
[website](https://ifconfig.co/) for full documentation and features.

## Usage
The most common use case would be to check your public ip:

```
curl ifconfig.co
```

However, you can obtain a lot more info about your connection:

```
curl ifconfig.co/city
curl ifconfig.co/country
curl ifconfig.co/json
```

## Tips
You can use [jq](https://stedolan.github.io/jq/) in order to format the json output of ifconfig.co

Just before we wrap this up, let me also add that you can check if your ports are exposed using this server also!

```
curl ifconfig.co/port/8080
```

## Links
- [Github](https://github.com/mpolden/echoip)
- [ifconfig.co](https://ifconfig.co/)