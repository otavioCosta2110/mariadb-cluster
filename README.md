# Mariadb cluster using kubernetes and galera.
<p align="center"> 
  <div align="center">
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flogodix.com%2Flogo%2F1886465.png&f=1&nofb=1&ipt=8101b5463a2f0a732d5d2a472a69c966050094db25b820058f819a88a6768521&ipo=images" style="width:20%; height:auto;">
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fblog.bosch-si.com%2Fwp-content%2Fuploads%2Fkubernetes-logo.png&f=1&nofb=1&ipt=82a2fb036b7496c0af2d94fe05acce4964576a4cb01c9692839b641ad3b389cd&ipo=images" style="width:20%; height:auto;">
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Faprenderbigdata.com%2Fwp-content%2Fuploads%2Fdocker-logo-1024x876.png&f=1&nofb=1&ipt=fbbae9dc13414e93e9262c60e60cb1a9a83499a4a5f5841037f3c2ec4a1ff5a6&ipo=images" style="width:20%; height:auto;">
    <img src="https://github.com/otavioCosta2110/mariadb-cluster/assets/106917785/fb58c2fa-0ffb-4bfb-ad60-2be53ad448ba" style="width:20%; height:auto;">    
  </div>
</p>

# What was used?
- Docker
- Kubernetes
- Mariadb (container)
- Galera (container)

# Notes on Kubernetes
- The number of pods being created are 3
- We have a service, a Stateful Set and a volume being shared by the pods
- The databases password is defined with this command: 
`kubectl create secret generic mariadb-galera-secret --from-literal=mariadb-root-password='your-database-password-here'`
