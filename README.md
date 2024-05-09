Para executar comandos no Kubernetes em modo de teste (dry-run), 
você pode usar o parâmetro `--dry-run=client` com o comando `kubectl`. 
Este parâmetro permite visualizar as alterações que seriam feitas sem realmente aplicá-las. 
Por exemplo, para criar um pod em modo de teste, você usaria o seguinte comando:

```bash
kubectl run pod-name --image=image-name --dry-run=client -o yaml
```

Este comando retorna a configuração yaml para o pod que seria criado, sem realmente criar o pod.
