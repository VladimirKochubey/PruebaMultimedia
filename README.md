PruebaMultimedia
================

Ejercicio cambios core de Liferay para edición inline de imágenes

Los cambios que he hecho

Cambiado
C:\Liferay\liferay-liferay-portal-11fe5a6\portal-web\docroot\WEB-INF\struts-config.xml

  	<action path="/document_library/edit_image_inline" type="com.liferay.portlet.documentlibrary.action.EditImageInlineAction">
			<forward name="portlet.document_library.edit_image_inline" path="portlet.document_library.edit_image_inline" />
			<forward name="portlet.document_library.error" path="portlet.document_library.error" />
		</action>

Cambiado
C:\Liferay\liferay-liferay-portal-11fe5a6\portal-web\docroot\WEB-INF\tiles-defs.xml

	<definition name="portlet.document_library.edit_image_inline" extends="portlet.document_library">
		<put name="portlet_content" value="/portlet/document_library/edit_image_inline.jsp" />
	</definition>


Cambiado
C:\Liferay\liferay-liferay-portal-11fe5a6\portal-web\docroot\html\portlet\document_library\view_file_entry.jsp


Añadido un fichero nuevo

C:\Liferay\liferay-liferay-portal-11fe5a6\portal-web\docroot\html\portlet\document_library\edit_image_inline.jsp


Añadido  un clase de Action

C:\Liferay\liferay-liferay-portal-11fe5a6\portal-impl\src\com\liferay\portlet\documentlibrary\action\EditImageInlineAction.java


Añadidos los claces en ficheros Language en

C:\Liferay\liferay-liferay-portal-11fe5a6\portal-impl\classes\content añadiendo

##
## Ejercicio
##

rotate-right = Rotar Derecha
rotate-left = Rotar Izquierda
edit-inline = Editar Imagen

etc.
