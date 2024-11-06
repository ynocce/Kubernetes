# Kubernetes

Principais Comandos Usados no Kubernetes: 

### 1. `kubectl get`
   - Exibe recursos, como `pods`, `services`, `nodes`, etc.
   - Exemplo: `kubectl get pods` lista todos os pods no namespace atual.

### 2. `kubectl describe`
   - Mostra detalhes completos de um recurso específico.
   - Exemplo: `kubectl describe pod <nome-do-pod>` exibe informações detalhadas sobre o pod.

### 3. `kubectl logs`
   - Visualiza os logs de um pod ou container específico.
   - Exemplo: `kubectl logs <nome-do-pod>` exibe os logs do pod.

### 4. `kubectl exec`
   - Executa comandos em um container dentro de um pod.
   - Exemplo: `kubectl exec -it <nome-do-pod> -- /bin/bash` abre um shell no container.

### 5. `kubectl apply`
   - Aplica ou atualiza configurações em um cluster com base em arquivos YAML.
   - Exemplo: `kubectl apply -f <arquivo.yaml>` cria ou atualiza recursos.

### 6. `kubectl delete`
   - Remove recursos do cluster.
   - Exemplo: `kubectl delete pod <nome-do-pod>` apaga o pod especificado.

### 7. `kubectl scale`
   - Ajusta o número de réplicas de um deployment ou outro recurso escalável.
   - Exemplo: `kubectl scale deployment <nome-do-deployment> --replicas=3` ajusta para 3 réplicas.

### 8. `kubectl expose`
   - Expõe um pod ou deployment como um serviço.
   - Exemplo: `kubectl expose deployment <nome-do-deployment> --type=LoadBalancer --port=80` cria um serviço do tipo LoadBalancer.

### 9. `kubectl port-forward`
   - Redireciona portas locais para um pod específico.
   - Exemplo: `kubectl port-forward pod/<nome-do-pod> 8080:80` redireciona a porta 8080 local para a porta 80 do pod.

### 10. `kubectl config set-context`
   - Define ou muda o contexto atual para conectar em um cluster específico.
   - Exemplo: `kubectl config set-context <nome-do-contexto>` altera o contexto.
