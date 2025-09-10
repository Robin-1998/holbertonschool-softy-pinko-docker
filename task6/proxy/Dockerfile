FROM nginx:latest

COPY proxy.conf /etc/nginx/conf.d/default.conf

# Le but de ton exercice est de centraliser l’accès à tes différents services (static server + API server)
# à travers un proxy unique, afin de simplifier la communication entre le front-end et le back-end, et
# éviter d’avoir à gérer plusieurs points d’accès ou adresses réseau.


# Un proxy, c’est un intermédiaire.
# Il reçoit les requêtes d’un client (par exemple un navigateur web) et les redirige vers un autre serveur (comme ton back-end ou front-end).
# Ensuite, il renvoie la réponse au client.

# Le rôle d’un proxy ici :

# Au lieu que ton navigateur parle directement à ton front-end ET à ton back-end,
# il parle seulement au proxy,
