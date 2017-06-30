# CakeLTE - CakePHP + AdminLTE 2

Versión de CakePHP con el template de AdminLTE 2

El ejemplo utiliza una base de datos llamada **cakephp** y una tabla llamada **usuarios** con la siguiente estructura:

```sql
CREATE TABLE `usuarios` (
  `id` int(10) UNSIGNED NOT NULL,
  `nombre` varchar(60) DEFAULT NULL,
  `apellido` varchar(60) DEFAULT NULL,
  `username` varchar(250) NOT NULL,
  `password` varchar(100) NOT NULL,
  `rol` varchar(20) NOT NULL DEFAULT 'user',
  `active` tinyint(1) NOT NULL DEFAULT '1',
  `created` datetime DEFAULT NULL,
  `modified` datetime DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


INSERT INTO `usuarios` (`id`, `nombre`, `apellido`, `username`, `password`, `rol`, `active`, `created`, `modified`) VALUES
(1, 'Roberto', 'WEST', 'rwest', '$2y$10$ZpjeiwMrGL6rU2e6m3Og7OBesu55iDA4xdn4gtLNQtzF7NSVwOTou', 'admin', 1, '2017-06-01 22:21:55', '2017-06-01 22:49:49'),
(2, 'Dario', 'MONTEROS', 'dmonteros', '$2y$10$2D5sT68gaElQwsaxi9F5sOVnCwjxvif3AQup5HuawdmcdxqtkAi3C', 'user', 1, '2017-06-01 22:50:24', '2017-06-01 22:50:24');


ALTER TABLE `usuarios`
  ADD PRIMARY KEY (`id`);

ALTER TABLE `usuarios`
  MODIFY `id` int(10) UNSIGNED NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=3;
```
