# Kops docker action

This action executes the kops binary.

## Inputs

**Required Environment Variables** 

NAME=myfirstcluster.example.com
AWS_ACCESS_KEY_ID=acess_key
AWS_SECRET_ACCESS_KEY=secret_key
AWS_DEFAULT_REGION=us-east-xxx
KOPS_STATE_STORE=s3://prefix-example-com-state-store


## Example usage

uses: nuvops/kops-cli@v1.16.2
env:
    AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
    AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    AWS_DEFAULT_REGION: ${{ secrets.AWS_REGION }}
    NAME: ${{ secrets.NAME }}
    KOPS_STATE_STORE: ${{ secrets.KOPS_STATE_STORE }}