# my helm chart repo

helm create demorepo

helm package ../demorepo

helm repo index .

helm repo list

helm repo add --username <github-user-name> --password <personel-access-token> my-github-repo 'https://raw.githubusercontent.com/<github-user-name>/my-chartrepo/main/demorepo'

helm repo list

helm push my-github-repo demorepo--0.1.0.tgz