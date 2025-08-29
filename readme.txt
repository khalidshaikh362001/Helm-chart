echo "# Helm-chart" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/khalidshaikh362001/Helm-chart.git
git push -u origin main

kubectl port-forward service/frontend-release-frontend-chart 30080:80 --address=0.0.0.0 &