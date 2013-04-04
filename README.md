businesslink assets
===================

This repository contains archived assets from businesslink.gov.uk. 

These are not deployed directly from git, but instead taken from the copy 
stored on S3. If changes are made, they can be synchronised with S3 like so:

    s3cmd -c ~/.ssh/s3cmd.conf sync --delete-removed businesslink/ s3://transition-assets/businesslink/
    s3cmd -c ~/.ssh/s3cmd.conf sync --delete-removed businesslink_improve/ s3://transition-assets/businesslink_improve/
    s3cmd -c ~/.ssh/s3cmd.conf sync --delete-removed businesslink_ukwelcomes/ s3://transition-assets/businesslink_ukwelcomes/

The s3 credentials are not stored in Github. Speak to a member of
ops or the Transition team to obtain them.
