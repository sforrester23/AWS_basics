# Setting up AWS: some basics

## Some things to do

1. Login to AWS, select S3
2. Set-up your instance: you need to get an SSH pair if you haven't already
3. Once it's running, we can ssh into it:

        ssh -i [location of key file] [user, e.g. ubuntu]@xxx-xx-xxx-xxx-xx.eu-west-2.compute.amazonaws.com

    We will now be in our vm.

4. We want to be able to move files into this area from our local machine.

        scp -i [location of key file] -r [location of file] [user, e.g. ubuntu]@xxx-xx-xxx-xxx-xx.eu-west-2.compute.amazonaws.com:[area to move it to]

5. We can now run our provision files that we have moved across, with ./provision.sh. Then we can have some nice provisioning to install necessary things in our machine.

6. We can also run tests.
