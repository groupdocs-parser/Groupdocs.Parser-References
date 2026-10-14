---
title: "com.groupdocs.parser.options"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Le package fournit des classes pour spécifier des options supplémentaires lors de l'analyse des données des documents."
type: docs
weight: 15
url: /fr/java/com.groupdocs.parser.options/
---

Le package fournit des classes pour spécifier des options supplémentaires lors de l'analyse des données des documents.



## Classes

| Classe | Description |
| --- | --- |
| [BarcodeOptions](../com.groupdocs.parser.options/barcodeoptions) | Fournit les options utilisées pour l'extraction de codes-barres. |
| [DocumentInfo](../com.groupdocs.parser.options/documentinfo) | Représente les informations du document. |
| [EmailConnection](../com.groupdocs.parser.options/emailconnection) | Représente les informations de connexion email. |
| [EmailEwsConnection](../com.groupdocs.parser.options/emailewsconnection) | Représente les informations de connexion email pour le protocole EWS. |
| [EmailImapConnection](../com.groupdocs.parser.options/emailimapconnection) | Représente les informations de connexion email pour le protocole IMAP. |
| [EmailPopConnection](../com.groupdocs.parser.options/emailpopconnection) | Représente les informations de connexion email pour le protocole POP. |
| [ExternalResourceHandler](../com.groupdocs.parser.options/externalresourcehandler) | Fournit un gestionnaire pour le chargement des ressources externes. |
| [ExternalResourceLoadingArgs](../com.groupdocs.parser.options/externalresourceloadingargs) | Fournit les données pour la méthode [ExternalResourceHandler.#onLoading(ExternalResourceLoadingArgs)](../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-). |
| [Features](../com.groupdocs.parser.options/features) | Représente la liste des fonctionnalités prises en charge. |
| [FileInfo](../com.groupdocs.parser.options/fileinfo) | Représente les informations du fichier. |
| [FileType](../com.groupdocs.parser.options/filetype) | Représente le type de fichier. |
| [FormattedTextOptions](../com.groupdocs.parser.options/formattedtextoptions) | Fournit les options utilisées pour l'extraction de texte formaté. |
| [HighlightOptions](../com.groupdocs.parser.options/highlightoptions) | Fournit les options utilisées pour extraire une mise en évidence (un bloc de texte autour du texte trouvé dans les scénarios de recherche). |
| [ImageOptions](../com.groupdocs.parser.options/imageoptions) | Fournit les options utilisées pour l'extraction d'images. |
| [LoadOptions](../com.groupdocs.parser.options/loadoptions) | Fournit les options utilisées pour ouvrir un fichier. |
| [OcrConnectorBase](../com.groupdocs.parser.options/ocrconnectorbase) | Fournit la fonctionnalité OCR. |
| [OcrEventHandler](../com.groupdocs.parser.options/ocreventhandler) | Fournit un gestionnaire pour les événements OCR. |
| [OcrOptions](../com.groupdocs.parser.options/ocroptions) | Fournit les options utilisées pour le connecteur OCR. |
| [PageAreaOptions](../com.groupdocs.parser.options/pageareaoptions) | Fournit les options utilisées pour l'extraction des zones de page. |
| [PageInfo](../com.groupdocs.parser.options/pageinfo) | Représente les informations de la page du document. |
| [PageRenderInfo](../com.groupdocs.parser.options/pagerenderinfo) | Représente les informations sur la façon dont une page est rendue. |
| [PageTableAreaOptions](../com.groupdocs.parser.options/pagetableareaoptions) | Fournit les options utilisées pour l'extraction des zones de tableau de page. |
| [PageTextAreaOptions](../com.groupdocs.parser.options/pagetextareaoptions) | Fournit les options utilisées pour l'extraction des zones de texte de page. |
| [ParserSettings](../com.groupdocs.parser.options/parsersettings) | Fournit les paramètres utilisés pour personnaliser l'extraction de données. |
| [PreviewOptions](../com.groupdocs.parser.options/previewoptions) | Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus. |
| [SearchOptions](../com.groupdocs.parser.options/searchoptions) | Fournit les options utilisées pour la recherche de texte. |
| [TextDocumentInfo](../com.groupdocs.parser.options/textdocumentinfo) | Représente les informations du document texte. |
| [TextOptions](../com.groupdocs.parser.options/textoptions) | Fournit les options utilisées pour l'extraction de texte. |

## Interfaces

| Interface | Description |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream) | Représente un délégué qui renvoie un flux pour écrire les données d'aperçu de page. |
| [IDocumentInfo](../com.groupdocs.parser.options/idocumentinfo) | Représente les informations du document. |
| [ILogger](../com.groupdocs.parser.options/ilogger) | Définit l'interface d'un logger utilisé pour consigner les événements et les erreurs lors de l'extraction de données. |
| [IPreviewPageRender](../com.groupdocs.parser.options/ipreviewpagerender) | Représente une méthode qui est appelée avant le rendu d'une page de document. |
| [IReleasePageStream](../com.groupdocs.parser.options/ireleasepagestream) | Représente une méthode qui libère le flux créé par le délégué [ICreatePageStream](../com.groupdocs.parser.options/icreatepagestream). |

## Énumérations

| Énum | Description |
| --- | --- |
| [FileFormat](../com.groupdocs.parser.options/fileformat) | Définit un type de fichier. |
| [FileTypeDetectionMode](../com.groupdocs.parser.options/filetypedetectionmode) | Définit un mode de détection du type de fichier. |
| [FormattedTextMode](../com.groupdocs.parser.options/formattedtextmode) | Définit un mode de texte formaté. |
| [ImageFormat](../com.groupdocs.parser.options/imageformat) | Définit un format d'image. |
| [PreviewFormats](../com.groupdocs.parser.options/previewformats) | Représente les formats d'aperçu pris en charge. |
| [QualityMode](../com.groupdocs.parser.options/qualitymode) | Définit un niveau de qualité. |
