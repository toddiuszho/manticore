Tricks
------

1. Edit `Gemfile.jruby-1.9.lock` if your dependency is locked down
2. Install dependencies and then gems
    
    env GEM_HOME=vendor/bundle/jruby/1.9 GEM_PATH="" vendor/jruby/bin/jruby -S gem install PATH_TO_DEPENDENCY_GEM
    bin/plugin install --no-verify PATH_TO_PLUGIN_GEM

Publishing
----------

1. Upload to files.RVT
2. Place in `/data/fileserve/gemserver/gems`
3. `gem generate_index -d /data/fileserve/gemserve`
