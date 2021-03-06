# eclipse_emsCad
# Requirements
- [es_extended](https://github.com/esx-framework/es_extended/tree/v1-final)

## Installation:
Put `eclipse_EmsCad` in your resources folder.
Ensure `eclipse_EmsCad` in your server cfg.
Insert sql dump(take in `eclipse_EmsCad`) in your db.
Add this columns to `users`:

![image](https://user-images.githubusercontent.com/36680471/129520235-3e8a542d-aaa6-4e72-a8a7-88fa20ebbc6b.png)



For change buttons key use `config.json`. `eclipse_cad/config.json`



For more questions douglasprod#6686 && https://discord.gg/8nXR6rfB2C


## Known Issues

1. Make sure you have `phone_number` in your db `users` table. And that it haven't null value

![image](https://user-images.githubusercontent.com/36680471/125207137-3c9e2880-e293-11eb-9083-031448fd0e5f.png)

If it have null value - CAD doesn't work


2. If you have something like this - problem with job_grades.  
![image](https://user-images.githubusercontent.com/36680471/125207153-4f186200-e293-11eb-80f9-e5f6831411ac.png)
![image](https://user-images.githubusercontent.com/36680471/125207162-5fc8d800-e293-11eb-9fb3-5d2ada6fd417.png)

Check `job_grades` table, if you have more job grades for police - you need make changes in source CAD files
![image](https://user-images.githubusercontent.com/36680471/129520361-71aad985-a5e4-4d83-98a0-68d74a4fa4d9.png)


2.1 Open esx_cad folder via VS Code. 

![image](https://user-images.githubusercontent.com/36680471/125207263-ee3d5980-e293-11eb-8901-782b2ddf4ce5.png)

2.2 Install node.js packages via command `npm install`

![image](https://user-images.githubusercontent.com/36680471/125207279-07dea100-e294-11eb-9b7e-88cd547ef36b.png)


2.3 Open `esx_cad/src/components/cad/PoliceCad.vue` 

2.4 Find `rankList`

![image](https://user-images.githubusercontent.com/36680471/129520405-8a6272ce-0016-4080-b467-0e1e5c0a4b4a.png)

2.5 Add ranks from your `job_grades` table

2.6 Compile Vue.js project via command `npm run build`

2.7 Take files from `ems_cad/dist` and move to your resource folder `eclipse_EmsCad/data`










