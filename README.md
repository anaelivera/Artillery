# Artillery
Performance test assignment
Para que el test funcione, es necesario ejecutar los siguiente en la terminal:
npm init -y
npm i artillery
export TOKEN="token de la api todoist"


Crear el siguiente script en el archivo package.json:
"test": "artillery run --output results/report.json performance.yml && artillery report --output results/report.html results/report.json"

Ejecutar en la terminal:
npm run test
