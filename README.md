# Production Docker deployment for Mattermost

This is an example repo with multiple Dockerfiles and a render.yaml for running a Mattermost server
with disk backed by PostgreSQL and Minio for uploaded artifacts such as images and videos.

You can fork this repo or click the Deploy to Render button below.

[![Deploy to Render](http://render.com/images/deploy-to-render-button.svg)](https://dashboard.render.com/iac/new?repoOwner=render-examples&repoName=mattermost&branch=master&provider=GITHUB)

The Deploy to Render button is not fully automated yet and requires you to copy the
`MINIO_ACCESS_KEY` and `MINIO_SECRET_KEY` environment variables from the `mattermost-minio` service
to the `MM_FILESETTINGS_AMAZONS3ACCESSKEYID` and `MM_FILESETTINGS_AMAZONS3SECRETACCESSKEY`
environment variables for the `mattermost` service.
