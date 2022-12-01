Esta ejecutando 5 contenedores: 
7271be28a648   nicopaez/jobvacancy-ruby:1.3.0   "/jobvacancy/start_a…"   3 minutes ago   Up 2 minutes   0.0.0.0:3000->3000/tcp   docker-kubernetes-web-1
4b4e1c2c6592   postgres:14.4-alpine             "docker-entrypoint.s…"   3 minutes ago   Up 3 minutes   5432/tcp                 docker-kubernetes-db-1
bcb041fceaa1   5021b0410677                     "ruby app.rb -o 0.0.…"   3 minutes ago   Up 3 minutes                            k8s_pingapp_pingapp-cd5565fc4-vj29g_default_9182cb0c-4ea1-46e5-9e77-2b3d2e17d163_3
c4e5dae7115d   5021b0410677                     "ruby app.rb -o 0.0.…"   3 minutes ago   Up 3 minutes                            k8s_pingapp_pingapp-cd5565fc4-zlskn_default_674af765-1aca-44f9-af5d-936df91b5a9d_1
e7db78e353f1   b30ba4516116                     "ruby app.rb -o 0.0.…"   3 minutes ago   Up 3 minutes                            k8s_pingapp_pingapp_default_e18a87a4-2420-45ad-a1ce-05093bd512a3_4

Esta basado en las imagenes: nicopaez/jobvacancy-ruby:1.3.0 y postgres:14.4-alpine, que incluyen la de ruby

Se leen entre los contenedores, porque utilizan el sistema operativo de la computadora y se pueden comunicar entre ellos a través de él
