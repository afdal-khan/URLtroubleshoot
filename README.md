# URLtroubleshoot


# urls for app (to make upload form)

from django.urls import path
from .views import index, RecordView

urlpatterns = [
    path('', index),
    path('records', RecordView.as_view())
]



# urls in main django project

urlpatterns=[
    url(r'^listings', index),
    #url(r'^detail', detail),
    url(r'^update/(?P<anime_id>[0-9]+)$', update),
   
]
   

