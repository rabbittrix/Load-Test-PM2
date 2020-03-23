## Cluster and Process Management with PM2

# Commands PM2:

pm2 start <index.js> //first start
kill -9 <2708>
pm2 ls //list de registers
pm2 reload index
pm2 stop index
pm2 start index //start after register
pm2 delete index // delete register of PM2
pm2 start index.js --name=echo // change the name of register
pm2 start index.js -i 0 // O (0) to trigger a process per CPU.
pm2 scale index 1 // choose the instance number
pm2 ecosystem simple // To test multiple applications
pm2 start ecosystem.config.js

# Load test with PM2 (npm i loadtest -g)

loadtest -c 100 -t 15 http://localhost:4000?message=hello
