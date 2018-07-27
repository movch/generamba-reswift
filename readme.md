# Generamba ReSwift Template

[Generamba](https://github.com/rambler-digital-solutions/Generamba) is a code generator made for working with Xcode. [ReSwift](https://github.com/ReSwift/ReSwift) template was made to simplify boilerplate code generation for each screen (actions, reducers, etc.).

## Installation

### Install Generamba

At present moment Generamba isn't maintained in main repository, so we have to use working fork. We'll also need [Specific Install gem](https://github.com/rdp/specific_install) to be able to install gems directly from repositories.

    sudo gem install "specific_install"
    sudo gem specific_install -l https://github.com/ladeiko/Generamba.git

If you don't have Rambafile, you'll need create it:

    generamba setup

### Install template

Add link to template to your Rambafile. For more information about Rambafile structure refer [Generamba wiki](https://github.com/rambler-digital-solutions/Generamba/wiki/Rambafile-Structure).

    templates:
    - {name: reswift, git: 'https://github.com/movch/generamba-reswift'}

Then execute command:

    generamba template install

## Usage

To generate template use the following command:

    generamba gen TemplateName reswift
