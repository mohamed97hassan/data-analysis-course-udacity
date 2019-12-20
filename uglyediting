select primary_poc, 
concat(left(primary_poc,strpos(primary_poc,' ')-1),'.',right(primary_poc,length(primary_poc)-strpos(primary_poc,' ')),'@',case when strpos(name,' ')= 0 then name else concat(left(name,strpos(name,' ')-1),right(name,length(name)-strpos(name,' '))) end,'.com') as mail,
concat(lower(left(primary_poc,1)),lower(right(left(primary_poc,strpos(primary_poc,' ')-1),1)),lower(left(right(primary_poc,length(primary_poc)-strpos(primary_poc,' ')),1)),lower(right(primary_poc,1)),length(left(primary_poc,strpos(primary_poc,' ')-1)),length(right(primary_poc,length(primary_poc)-strpos(primary_poc,' '))),upper(case when strpos(name,' ')= 0 then name else concat(left(name,strpos(name,' ')-1),right(name,length(name)-strpos(name,' '))) end)     )
from accounts 
