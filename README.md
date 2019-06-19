# travis-jdk-switch-test

Test to find what JDKs are available in Travis now.

Troubleshooting recent build failures:

```
$ export JAVA_HOME=~/oraclejdk8
$ export PATH="$JAVA_HOME/bin:$PATH"
$ ~/bin/install-jdk.sh --target "/home/travis/oraclejdk8" --workspace "/home/travis/.cache/install-jdk" --feature "8" --license "BCL"
install-jdk.sh 2019-05-02
Expected feature release number in range of 9 to 14, but got: 8
```