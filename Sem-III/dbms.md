```sql

select e.name as name,
sum(d.amount) as balance 
from Users e join Transactions d on e.account=d.account
group by e.name having balance>10000

```
