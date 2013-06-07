When running `ruby myapp.rb` (after bundling), I get this:

    1 ⮀ neo4j_ha ⮀ ruby myapp.rb
    ‹jruby-1.6.7@sheldon› ∞
    ha.initial_hosts: localhost:5001,localhost:5002,localhost:5003
    I, [2013-06-07T17:44:56.004000 #76486]  INFO -- : starting Neo4j in HA
    mode, machine id: 1 at localhost:6001 db
    /Users/jannis/Dev/school/neo4j_ha/db/neo1
    NameError: cannot load Java class
    org.neo4j.graphdb.factory.HighlyAvailableGraphDatabaseFactory
               for_name at org/jruby/javasupport/JavaClass.java:1205
        get_proxy_class at org/jruby/javasupport/JavaUtilities.java:34
          const_missing at
    /Users/jannis/.rvm/rubies/jruby-1.6.7/lib/ruby/site_ruby/shared/builtin/javasupport/java.rb:45
      start_ha_graph_db at
    /Users/jannis/.rvm/gems/jruby-1.6.7@sheldon/gems/neo4j-core-2.2.4-java/lib/neo4j-core/database.rb:188
                  start at
    /Users/jannis/.rvm/gems/jruby-1.6.7@sheldon/gems/neo4j-core-2.2.4-java/lib/neo4j-core/database.rb:62
                  start at
    /Users/jannis/.rvm/gems/jruby-1.6.7@sheldon/gems/neo4j-core-2.2.4-java/lib/neo4j-core/database.rb:53
                  start at
    /Users/jannis/.rvm/gems/jruby-1.6.7@sheldon/gems/neo4j-core-2.2.4-java/lib/neo4j/neo4j.rb:41
                  start at myapp.rb:21
                 (root) at myapp.rb:24
     1 ⮀ neo4j_ha
