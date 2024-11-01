# YAML anchors 

The YAML anchors allows us to duplicate contents across the config file.
This can be used to inherit properties.

```
base: &base
    tag: same tag

child:
    <<: *base
    another key: 10
```

will insert all the key values from base under child.
