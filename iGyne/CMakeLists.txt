#-----------------------------------------------------------------------------
set(MODULE_NAME iGyne)

#-----------------------------------------------------------------------------
set(MODULE_PYTHON_SCRIPTS
  ${MODULE_NAME}.py
  )

set(MODULE_PYTHON_RESOURCES
  ${MODULE_NAME}Wizard/__init__.py
  ${MODULE_NAME}Wizard/Helper.py
  ${MODULE_NAME}Wizard/iGyneStep.py
  ${MODULE_NAME}Wizard/iGyneFirstRegistrationStep.py
  ${MODULE_NAME}Wizard/iGyneLoadModelStep.py
  ${MODULE_NAME}Wizard/iGyneNeedlePlanningStep.py
  ${MODULE_NAME}Wizard/iGyneNeedleSegmentationStep.py
  ${MODULE_NAME}Wizard/iGyneSecondRegistrationStep.py
  ${MODULE_NAME}Wizard/iGyneSelectApplicatorStep.py
  ${MODULE_NAME}Wizard/iGyneSelectProcedureStep.py
  )

#-----------------------------------------------------------------------------
slicerMacroBuildScriptedModule(
  NAME ${MODULE_NAME}
  SCRIPTS ${MODULE_PYTHON_SCRIPTS}
  RESOURCES ${MODULE_PYTHON_RESOURCES}
  )

