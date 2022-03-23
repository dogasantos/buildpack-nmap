# buildpack-nmap

(forked from hahwul/buildpack-nmap)

Updates:

* new nmap version
* build with old openssl that supports old algos (like sha256)
* build with nmap datadir (NSE scripts support)

Now you can just set the datadir as "/app/nmap/nmapdatadir/nmap" and the script engine will work.


<a href="https://heroku.com/deploy?template=https://github.com/dogasantos/buildpack-nmap">
  <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy">
</a><br>
install nmap and set alias buildpack of heroku for me(add export ENV)

## Composed
```
$ heroku create --buildpack  https://github.com/dogasantos/buildpack-nmap.git
$ git push heroku master
```
## setting config vars
`App => Settings => Config vars`
<img src="https://user-images.githubusercontent.com/13212227/65061836-b5910980-d9b5-11e9-94d4-4cb5b20929a7.png">

## References
https://github.com/socialpaymentsbv/heroku-buildpack-nmap
