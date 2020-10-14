## Repositories

* Đây là thư mục khởi tạo cho pattern Repositories dùng trong Laravel

### Sử dụng

* Bạn chỉ cần copy các file của thư mục vào trong thư mục `Repositories` của bạn

* Khi tạo mới file Repositories cho dự án của bạn chỉ cần nhúng đường dẫn của file `RespositoryAbstract` theo cách như sau:
   ```php
    <?php
        namespace App\Repositories\Frontend;
        use App\Respositories\RespositoryAbstract;
        use App\Models\Brand;

        /**
        * Class BrandRepository
        *
        * @package App\Repositories\Backend
        * @author EnableStartup <hello@enablestartup.com>
        */
        class BrandRepository extends RespositoryAbstract
        {

            /**
            * Function getModel
            *
            * @return model
            */
            public function getModel()
            {
                return Brand::class;
            }
        }
    ```
