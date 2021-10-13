# laravel-todolist
Lista de tareas hecha con Laravel y Vue



CONSULTA SQL

Promedio de articulos por oficina
SELECT AVG(op.quantity) FROM outputproducts op
JOIN users u ON (op.user_id = u.id) 
WHERE op.product_id = 20 
AND u.area_id = 37
AND EXTRACT(YEAR FROM op.output_date) = 2021
AND EXTRACT(MONTH FROM op.output_date) = 10
AND op.quantity>0
