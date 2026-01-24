## Paso 0: Vinculación
gcloud init

## Paso 1: Creación del repositorio en Artifact Registry (GCP)
gcloud artifacts repositories create repo-mlops14-streamlit-ml --repository-format docker --project mlops-14-project-deploy-fast --location us-central1

## Paso 2: Crear el repo de github

## Paso 3: Crear la Key de la Cuenta de Servicio

## Paso 4: Colocar el Service Account Key en GitHub Settings

## Paso Automatizacion:
- git init
- git add .
- git commit -m "Proyecto de automatización de despliegue en GCR"
- git branch -M main
- git remote add origin https://github.com/KevinInoCol/mlops-14-ml-regression-casas-streamlit.git
- git push -u origin main



## Cuando deseas volver a subir por algun error corres lo siguiente:
- git remote remove origin

- git add .
- git commit -m "Correccion3"
- git push origin main












## Paso 4: OPCIONAL, Dar permisos de acceso a mi APLICACION. ESTO SE EJECUTA UNA SOLA VEZ
gcloud run services set-iam-policy servicio-streamlit-sesion3-kevin-inofuente gcr-service-policy.yaml --region us-central1 --project project-mlops-10-streamlit