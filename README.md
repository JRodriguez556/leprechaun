# Leprechaun

The purpose of this tool is to help penetration testers identify potentially valuable targets on the internal network environment. By aggregating netstat routes from multiple hosts, you can easily figure out what services and servers they're connected to.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

You'll need a few Ruby gems to get started -- if you don't have them already, that is.

```
gem install 'securerandom'
gem install 'terminal-table'
gem install 'getopt'
```

### Tool help menu

If you run the script without any arguments, you'll be provided with the following help menu:

```
[root:vonahisec-kali:~/scripts/leprechaun]# ./leprechaun.rb

 -------------------------------------------------------------
 Leprechaun v1.0 - Alton Johnson (@altonjx)
 -------------------------------------------------------------

  Usage: ./leprechaun.rb -f /path/to/netstat_results.txt -p <port>

  -f	File containing the output of netstat results.
  -p	Port you're interested in. E.g., 80. Specify "all" to see all traffic or "common" for common ports.

  Example: ./leprechaun.rb -f netstat_output.txt -p 80
  Example: ./leprechaun.rb -f netstat_output.txt -p all
  Example: ./leprechaun.rb -f netstat_output.txt -p common
```

## Additional References

Blog post: 

## Authors

* **Alton Johnson** - *Initial work* - [Twitter](https://www.twitter.com/altonjx)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments & Credits

* Josh Stone - Influenced by Routehunter