# README

## Pasos

	1.- create a main branch
	2.- create a gh-pages branch
	3.- create a feature branch

## check CRDs version

	kubectl get crd  | grep external

	kubectl describe crd externalsecrets.external-secrets.io

## Loging

-- login

	helm registry login  

-- privado

	helm repo add argocd-helm-charts https://raw.githubusercontent.com/XSell/argocd-helm-charts/gh-pages --username pepe --password pepe  

-- publico

	helm repo add argocd-helm-charts https://raw.githubusercontent.com/XSell/argocd-helm-charts/gh-pages  

-- pull

	helm dependency build  

## Test

	helm upgrade dummy --install . -f values-example.yaml --dry-run --debug

	helm upgrade dummy --install . -f values-example.yaml

## clouds

	Helms Versions :

		- base
