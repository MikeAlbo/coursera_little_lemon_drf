# coursera_little_lemon_drf

Coursera Django rest frame work API project

--------

A basic CRUD app using the Django Rest Framework and SQLite. Utilizes class based routing with generics

*e.g.*

```python
class SingleMenuItemView(generics.RetrieveUpdateAPIView, generics.DestroyAPIView):
    queryset = MenuItem.objects.all()
    serializer_class = MenuItemSerializer
```

```python
urlpatterns = [
    path('menu-items', views.MenuItemsView.as_view()),
    path('menu-items/<int:pk>', views.SingleMenuItemView.as_view()),
]
```

# packages used

- [Django Rest Framework](https://www.django-rest-framework.org/)
- [Django Debug Toolbar](https://django-debug-toolbar.readthedocs.io/en/latest/installation.html)

