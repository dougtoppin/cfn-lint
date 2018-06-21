# cfn-lint
Useful AWS CloudFormation python-cfn-lint utility for checking templates

I don't like to have to install and maintain tools locally if I can avoid it so I try to run tools in containers instead.

This repo is used to build a Dockerhub image of the python-cfn-lint tool.

### Usage

Run this using the image like this:

    docker run -t -v $(pwd):/tmp dougtoppin/cfn-lint:1.0 cloudformation_template_file

Make it easier by setting up a shell alias like this:

    alias cfn-lint="docker run -t -v $(pwd):/tmp dougtoppin/cfn-lint:1.0 "

Once the alias has been created use it like this:

    cfn-lint cloudformation_template_file

### Details on the tool

More on the tool at [https://github.com/awslabs/cfn-python-lint](https://github.com/awslabs/cfn-python-lint)
