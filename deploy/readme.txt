
- Run './build rebuild' from the root to build 'jline/target/jline-3.20.1.jar'.

# Deploy locally:
clojure -X:install

# Deploy to Clojars (replace username + clojars-token):
env CLOJARS_USERNAME=username CLOJARS_PASSWORD=clojars-token clojure -X:deploy
