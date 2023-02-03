# SQL/결과

# 8월 이후 접종자
# SELECT a.inocu_date , b.name FROM inoculator AS a INNER JOIN person AS b ON a.person_id = b.person_id WHERE date_format(a.inocu_date, "%m")>= "08"

# 결핵 접종 받은 고객의 접종 일자, 이름
# SELECT a.name, b.inocu_date, c.vac_name FROM person AS a INNER JOIN inoculator AS b ON a.person_id  = b.person_id INNER JOIN vaccine AS c ON b.vac_code = c.vac_code WHERE c.vac_name = "결핵"

# 예약자의 전자문진 작성 날짜, 예약 날짜, 이름
# SELECT c.name, b.dat, a.reser_date FROM reser AS a INNER JOIN electronic_examination AS b ON a.elect_code = b.elect_code INNER JOIN person AS c ON c.person_id = a.person_id



