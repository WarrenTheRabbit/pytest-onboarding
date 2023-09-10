`NodeMeta` is a metaclass for `Node`.

It forces Nodes to be instanatiated with the named constructor `from_parent`. By limiting the api surface, it enables better/simpler refactoring of the collection tree.

