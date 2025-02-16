# proyecto-github
PASOS REALIZADOS:
1. Crear repositorio en github
git init proyecto-github
2. Clonar repositorio local
git clone https://github.com/priscilabreu05/proyecto-github
cd proyecto-github
3. Crear archivos index.html y readme.md
4. First commit
git add .
git commit -m "first commit"
5. Modificar index.html agregando una etiqueta h1
6. Commit de agregado titulo
git add index.html
git commit -m "Agregado título"
8. Usar git log y guardar el hash del primer commit en log_com.txt
git log --oneline
echo "Primer commit hash: fcef088" > log_com.txt
9. Crear la rama "estilos"
git branch estilos
git checkout estilos
10. Añadir styles.css y darle estilos al titulo
11. Modificar index.html para enlazar styles.css
12. Commit de agregado css
git add .
git commit -m "Agregado CSS"
13. Fusionar estilos en main
git checkout main
git merge estilos
15. Usar git reset para eliminar el último commit SIN PERDER ARCHIVOS
git reset --soft HEAD~1
16. Explicar en log_com.txt qué comando se utilizó y por qué
17. Usar git checkout para ver cómo era el proyecto en el commit cuyo hash se guardó en log_com.txt
git checkout fcef088
18. Volver a la última versión con git checkout main
git checkout main
