FROM nginx:alpine
# Bake the nginx config template into the image. Coolify turns single-file bind
# mounts into empty directories, which breaks the original ./nginx/nginx.conf mount
# (nginx then can't start: "cp: can't stat .../nginx.conf.template: Not a directory").
COPY nginx/nginx.conf /etc/nginx/nginx.conf.template
