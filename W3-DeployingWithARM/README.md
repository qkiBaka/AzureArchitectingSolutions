# Week 3
## To Do:
### Opis sytuacji
Jesteś architektem w firmie o europejskim zasięgu i rozpoczynasz w swojej firmie budowanie rozwiązań opartych o Microsoft Azure.  
Jako architekt ustaliłeś kilka pryncypiów projektowych, które powinny być respektowane przy każdym wdrożeniu:  
Każdy projekt powinien używać konwencji nazw dla grup i zasobów zgodnych z konwencją firmy  
Infrastruktura, budowana w Azure pod środowiska czy aplikacje powinna być zawsze budowana z wykorzystaniem Azure Resource Managera i template’ów. Jeśli jest to duże wdrożenie, powinny być użyte tzw. Linked Templates.  
Jeśli to konieczne, należy zbudować własny model ról za pomocą RBAC  
Docelowo, wszystkie kluczowe ustawienia, tak jak np. nazwy lokalnych administratorów i hasła powinny być pobierane z Azure KeyVault  
### TYDZIEN3.1 
„Zbuduj prostą konwencję nazewniczą dla min. takich zasobów jak Grupa Zasobów, VNET, Maszyn Wirtualna, Dysk, Konta składowania danych. Pamiętaj o ograniczeniach w nazywaniu zasobów, które występują w Azure”  
### TYDZIEN3.2   
„Zbuduj prosty ARM Template (możesz wykorzystać już gotowe wzorce z GitHub), który wykorzystuje koncepcję Linked Templates. Template powinien zbudować środowisko złożone z jednej sieci VNET, podzielonej na dwa   subnety. W każdy subnecie powinna powstać najprostsza maszyna wirtualna z systemem Ubuntu 18.04 a na każdym subnecie powinny zostać skonfigurowane NSG.”  

### TYDZIEN3.3 
„Zbuduj najprostrzą właśną rolę RBAC, która pozwala użytkownikowi uruchomić maszynę, zatrzymać ją i zgłosić zgłoszenie do supportu przez Portal Azure”  

### TYDZIEN3.4 
„Spróbuj na koniec zmodyfikować template tak, by nazwa użytkownika i hasło do każdej maszyny z pkt. 2 było pobierane z KeyVault.  

## Notes:
### RBAC:
https://docs.microsoft.com/en-us/azure/role-based-access-control/overview  
https://docs.microsoft.com/en-us/azure/role-based-access-control/custom-roles  
https://docs.microsoft.com/en-us/azure/role-based-access-control/custom-roles-powershell  
https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitoring-overview-activity-logs  

### Deploy with ARM:
https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-authoring-templates  
https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview  
### Naming conventions:  
### Restrictions:
https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/resource-name-rules  

### Recommendations:
https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/naming-and-tagging  
https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-best-practices/resource-naming  

### Ready blocks:
https://github.com/Azure/azure-quickstart-templates  
https://github.com/mspnp/template-building-blocks  

### Using key-vault for ARM:
https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/parameter-files  