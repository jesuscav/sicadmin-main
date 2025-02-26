<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Documentación para el Formulario de Gestión de Cuentas del Paciente</title>
</head>
<body>
    <h2>Documentación para el Formulario de Gestión de Cuentas del Paciente</h2>
    <h3>1. Descripción General</h3>
    <p>El formulario de gestión de cuentas del paciente permite gestionar los gastos de servicios internos y externos así como los honorarios médicos asociados a un paciente. Aquí registramos los ítems que en la cuenta creada por la historia. Estos pueden venir de Emergencia al pasar el paciente a hospitalizado. Esta agrupa los cargos de los servicios si es integrado con Laboratorio, Imágenes, RX y Almacén. Los ítems aparecerán referenciados por el número de registro que lo originó, así un cargo de RX tendrá una numeración que se envía a hospitalización y se agrega el grupo y su número que lo generó, de tal manera que este recibo indica su origen junto con su servicio. Todos los ítems agrupados pueden imprimir su desglose que lo componen.</p>
    <h3>2. Campos del Formulario</h3>
    <h4>2.1. Información del Paciente y Responsable</h4>
    <ul>
        <li><strong>Paciente</strong>: Nombre del paciente.</li>
        <li><strong>Idx</strong>: Identificador único del paciente.</li>
        <li><strong>Responsable Seguro / Médico</strong>: Nombre del responsable del seguro o médico.</li>
        <li><strong>Datos de Impresión</strong>: Información adicional para la impresión de la factura.</li>
    </ul>
    <h4>2.2. Detalles de la Factura</h4>
    <ul>
        <li><strong>Código Servicio</strong>: Código del servicio médico.</li>
        <li><strong>No. Cuenta</strong>: Número de cuenta asociado al paciente.</li>
        <li><strong>Historia</strong>: Número de historia clínica.</li>
        <li><strong>No. Factura</strong>: Número de la factura.</li>
        <li><strong>Fec. de Ingreso</strong>: Fecha de ingreso del paciente.</li>
        <li><strong>IPTASA</strong>: Tasa aplicada.</li>
        <li><strong>Pre Factura</strong>: Monto antes de la factura.</li>
        <li><strong>Estado</strong>: Estado de la factura (Pendiente, Pagada, etc.).</li>
        <li><strong>Cédula</strong>: Número de cédula del paciente.</li>
        <li><strong>Fec. de Egreso</strong>: Fecha de egreso del paciente.</li>
        <li><strong>Fec. de Factura</strong>: Fecha de la factura.</li>
        <li><strong>Coma. Pago</strong>: Comentarios sobre el pago.</li>
        <li><strong>Descripción</strong>: Descripción adicional de la factura.</li>
    </ul>
    <h4>2.3. Montos y Totales</h4>
    <ul>
        <li><strong>MONTO EXENTO</strong>: Monto exento de impuestos.</li>
        <li><strong>MONTO DESCUENTO</strong>: Monto de descuento aplicado.</li>
        <li><strong>MONTO IVA</strong>: Monto del IVA.</li>
        <li><strong>TOTAL FACTURADO</strong>: Total facturado.</li>
        <li><strong>MONTO IGTE</strong>: Monto de otros impuestos.</li>
        <li><strong>MONTO COBRADO</strong>: Monto cobrado.</li>
        <li><strong>TOTAL SALDO</strong>: Saldo total pendiente.</li>
    </ul>
    <h4>2.4. Detalles de Recibos</h4>
    <ul>
        <li><strong>Lín</strong>: Línea de detalle.</li>
        <li><strong>Código</strong>: Código del servicio o producto.</li>
        <li><strong>Monito</strong>: Monto individual.</li>
        <li><strong>Total Monto</strong>: Monto total.</li>
        <li><strong>No. Recibo</strong>: Número de recibo.</li>
        <li><strong>Ser</strong>: Serie del recibo.</li>
    </ul>
    <h3>3. Instrucciones para Completar el Formulario</h3>
    <ol>
        <li><strong>Información del Paciente y Responsable</strong>:
            <ul>
                <li>Ingrese el nombre del paciente, el identificador único (Idx), y el nombre del responsable del seguro o médico.</li>
                <li>Proporcione cualquier información adicional necesaria para la impresión de la factura.</li>
            </ul>
        </li>
        <li><strong>Detalles de la Factura</strong>:
            <ul>
                <li>Complete el código del servicio, número de cuenta, número de historia clínica, número de factura, fecha de ingreso, tasa aplicada (IPTASA), monto antes de la factura, estado de la factura, cédula del paciente, fecha de egreso, fecha de la factura, comentarios sobre el pago y una descripción adicional.</li>
            </ul>
        </li>
        <li><strong>Montos y Totales</strong>:
            <ul>
                <li>Ingrese el monto exento, monto de descuento, monto del IVA, total facturado, monto de otros impuestos, monto cobrado y el saldo total pendiente.</li>
            </ul>
        </li>
        <li><strong>Detalles de Recibos</strong>:
            <ul>
                <li>Proporcione los detalles de cada recibo, incluyendo la línea de detalle, código del servicio o producto, monto individual, monto total, número de recibo y serie del recibo.</li>
            </ul>
        </li>
    </ol>
    <h3>4. Validaciones y Restricciones</h3>
    <ul>
        <li><strong>Campos Obligatorios</strong>: Paciente, Idx, Código Servicio, No. Cuenta, No. Factura, Fec. de Ingreso, Estado, Cédula, Fec. de Egreso, Fec. de Factura, MONTO EXENTO, MONTO DESCUENTO, MONTO IVA, TOTAL FACTURADO, MONTO IGTE, MONTO COBRADO, TOTAL SALDO.</li>
        <li><strong>Formato de Fecha</strong>: Las fechas deben estar en formato DD/MM/AAAA.</li>
        <li><strong>Longitud Máxima</strong>:
            <ul>
                <li>Nombre del Paciente: 100 caracteres.</li>
                <li>Código Servicio: 20 caracteres.</li>
                <li>No. Cuenta: 15 caracteres.</li>
                <li>No. Factura: 15 caracteres.</li>
                <li>Descripción: 200 caracteres.</li>
            </ul>
        </li>
    </ul>
    <h3>5. Ejemplo de Interfaz</h3>
    <p><img src="images/EDOCUENTAHOSP/CEdoCuentaHosp.JPG" alt="Estado de cuenta del paciente"></p>
    <h3>6. Flujo de Trabajo</h3>
    <ol>
        <li>El usuario ingresa la información del paciente y los detalles de la factura en los campos correspondientes.</li>
        <li>El usuario ingresa los montos y totales asociados a la factura.</li>
        <li>El usuario proporciona los detalles de los recibos.</li>
        <li>El usuario hace clic en "Guardar" para registrar la información.
            <ul>
                <li>Si los campos obligatorios están completos y válidos, la información se registra en el sistema.</li>
                <li>Si hay errores, se muestran mensajes de validación.</li>
            </ul>
        </li>
        <li>El usuario puede hacer clic en "Cancelar" para limpiar el formulario y descartar los cambios.</li>
    </ol>
    <h3>7. Pruebas</h3>
    <ul>
        <li><strong>Caso 1</strong>: Completar todos los campos obligatorios y hacer clic en "Guardar". Resultado esperado: Registro exitoso.</li>
        <li><strong>Caso 2</strong>: Dejar campos obligatorios vacíos y hacer clic en "Guardar". Resultado esperado: Mensajes de error.</li>
        <li><strong>Caso 3</strong>: Hacer clic en "Cancelar". Resultado esperado: Limpiar el formulario.</li>
    </ul>
</body>
</html>
