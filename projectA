-- 従業員テーブルの作成
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    department VARCHAR(50),
    salary DECIMAL(10,2),
    hire_date DATE
);

-- データの挿入
INSERT INTO employees (id, name, department, salary, hire_date) VALUES
(1, '田中 太郎', '営業', 5000000, '2020-04-01'),
(2, '佐藤 花子', '開発', 6000000, '2018-07-15'),
(3, '鈴木 一郎', '人事', 4500000, '2019-09-10');

-- 給与が500万円以上の従業員を取得
SELECT * FROM employees WHERE salary >= 5000000;

-- 部署ごとの平均給与を算出
SELECT department, AVG(salary) AS average_salary
FROM employees
GROUP BY department;

-- 従業員の情報を更新（ID=1の人の給与を550万円に変更）
UPDATE employees SET salary = 5500000 WHERE id = 1;

-- 従業員データの削除（ID=3の人を削除）
DELETE FROM employees WHERE id = 3;
