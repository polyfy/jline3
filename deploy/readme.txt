
# Make sure you have built 'jline/target/jline-3.20.1.jar'
# From the root of this repository, execute:
./build rebuild

# From this directory, install locally to ~/.m2/repository/com/github/polyfy/jline/3.20.1:
clojure -X:install

# Deploy to Clojars (replace username + clojars-token):
env CLOJARS_USERNAME=username CLOJARS_PASSWORD=clojars-token clojure -X:deploy

# Use from deps.edn:
:extra-deps {
  com.github.polyfy/jline {:mvn/version "3.20.1"}
}
