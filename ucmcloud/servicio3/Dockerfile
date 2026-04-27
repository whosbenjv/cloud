FROM node:20

WORKDIR /app

# 🔥 instalar Angular CLI
RUN npm install -g @angular/cli

# 🔥 crear proyecto Angular dentro del contenedor
RUN ng new mi-angular-app --defaults --skip-git

WORKDIR /app/mi-angular-app

# instalar dependencias
RUN npm install

EXPOSE 4200

CMD ["ng", "serve", "--host", "0.0.0.0", "--port", "4200"]