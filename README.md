# hello-branch
test

-- GPDB master, segment node configuration 확인
select * from pg_catalog.gp_segment_configuration;

-- MADlib 버전 확인
select madlib.version();
select * from madlib.migrationhistory;
-- PL/Language
select * from pg_catalog.pg_language;

데이터 크기가 로컬 컴퓨터의 메모리 한계를 벗어날 정도로 크다면 
그때는 DB에서 SQL로 집계를 한 후, 집계 결과만을 Python이나 R로 가져와서 시각화를 하는 방법


DROP TABLE IF EXISTS houses;
CREATE TABLE houses (id INT, tax INT, bedroom INT, bath FLOAT, price INT,
            size INT, lot INT);
INSERT INTO houses VALUES
  (1 ,  590 ,       2 ,    1 ,  50000 ,  770 , 22100),
  (2 , 1050 ,       3 ,    2 ,  85000 , 1410 , 12000),
  (3 ,   20 ,       3 ,    1 ,  22500 , 1060 ,  3500),
  (4 ,  870 ,       2 ,    2 ,  90000 , 1300 , 17500),
  (5 , 1320 ,       3 ,    2 , 133000 , 1500 , 30000)
SELECT * FROM houses;
