# Vagrant AWS Provider (Community Maintained Fork)

**Original Repository:** [https://github.com/mitchellh/vagrant-aws](https://github.com/mitchellh/vagrant-aws)
This repository is a community-maintained fork of the original `mitchellh/vagrant-aws` provider, which was archived on Feb 11, 2022. The original project is read-only.

This fork aims to provide continued support and compatibility with modern systems and Vagrant versions, addressing issues that prevented the original plugin from installing and functioning correctly. All credit for the original work goes to Mitchell Hashimoto and the `vagrant-aws` contributors.

## What's New in this Fork?

This fork includes patches to resolve installation issues on modern systems and ensure compatibility with current Vagrant environments. Specifically, it addresses problems that prevented `vagrant plugin install vagrant-aws` from succeeding after the original repository was archived.


## Usage (with this Fork)

Since the original plugin is no longer maintained and available on RubyGems, you'll need to install this fork directly from the `.gem` file you build.

1.  **Build the Gem:**
    ```bash
    gem build vagrant-aws.gemspec
    ```

2.  **Install the Plugin:**
    ```bash
    vagrant plugin install ./vagrant-aws-0.7.2.gem # (Verify the version number in vagrant-aws.gemspec)
    ```

3.  **Add the Dummy Box:**
    ```bash
    vagrant box add aws-dummy [https://github.com/mitchellh/vagrant-aws/raw/master/dummy.box](https://github.com/mitchellh/vagrant-aws/raw/master/dummy.box)
    ```
    
  
For detailed configuration options and examples, please refer to the original documentation - [https://github.com/mitchellh/vagrant-aws](https://github.com/mitchellh/vagrant-aws)
