include(FindGettext)

foreach(lang ca cs de es fr it ja ko pa pl pt_BR uk zh_CN zh_TW)
    GETTEXT_PROCESS_PO_FILES(${lang} ALL
        INSTALL_DESTINATION ${CMAKE_INSTALL_LOCALEDIR}
        PO_FILES ${lang}.po)
endforeach()

