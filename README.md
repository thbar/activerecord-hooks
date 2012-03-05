This repository is a place to discuss the current needs to extend ActiveRecord and see if we can provide a clean, shared way to achieve this.

### Some background

[adapter_extensions](https://github.com/activewarehouse/adapter_extensions) is a gem that add features to ActiveRecord adapters. It started in 2006 and is currently maintained by Thibaut Barrère.

Upgrading adapter_extensions to Rails 3 wasn't trivial, so the maintainer looked for a solution and discovered [activerecord-import](https://github.com/zdennis/activerecord-import) by Zach Dennis, which implemented a trick to extend ActiveRecord adapters.

After chatting a bit, we came to the conclusion that it would be useful to create a common solution to extend ActiveRecord.

### TODO

* write down the current use-cases
* define ActiveRecord hooks or other tricks which would let us extend as needed
* create a gem that will solve that
* eventually, merge the gem into Rails itself